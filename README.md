MainActivity отвечает за инициализацию MainFragment при первом запуске приложения. MainFragment содержит пользовательский интерфейс и логику представления данных. В этом фрагменте также создается экземпляр ViewModel, который используется для управления данными.

MainViewModel управляет данными и бизнес-логикой. Она использует GetUsefulActivityUseCase для получения данных о полезной деятельности.

MainViewModelFactory создаёт экземпляры MainViewModel для ViewModelProvider.

GetUsefulActivityUseCase определяет метод execute, который будет использоваться для получения данных о полезной деятельности.

AppComponent предоставляет зависимости для всего приложения.

DataModule предоставляет реализацию UsefulActivitiesRepository.

PresentationModule предоставляет реализации MainViewModel и MainViewModelFactory.

UsefulActivitiesRepository отвечает за получение данных о полезной деятельности из внешнего источника (в данном случае через HTTP-запрос к API).

State представляет состояние данных. Он используется в MainViewModel для управления состоянием данных.

UsefulActivityDto является моделью данных, которая используется для представления данных о полезной деятельности.

