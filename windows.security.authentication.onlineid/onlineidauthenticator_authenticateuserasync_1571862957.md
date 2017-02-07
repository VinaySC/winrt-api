---
-api-type: winrt method
---
 If the asynchronous authentication request fails, the error is captured in the errorcode of the [IAsyncInfo](http://msdn.microsoft.com/library/3444e02e-8817-4c23-84d9-1a2d1bf43a52) object.
 If the asynchronous authentication requests starts and some of the tickets were obtained but some of them failed, the response is S_OK.
 If the authentication request itself succeeded but individual tickets couldn’t be requested, [IAsyncInfo](http://msdn.microsoft.com/library/3444e02e-8817-4c23-84d9-1a2d1bf43a52) returns S_OK but [OnlineIdServiceTicket.ErrorCode](onlineidserviceticket_errorcode.md) captures individual ticket error codes.
 If all of the ticket requests failed, the [IAsyncInfo](http://msdn.microsoft.com/library/3444e02e-8817-4c23-84d9-1a2d1bf43a52) will contain the actual error code.
 If all calls succeeded and all of the tickets were successfully obtained, the error code will be S_OK indicating no error occurred .