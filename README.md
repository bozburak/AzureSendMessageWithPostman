English
This JSON is a Postman collection that sends a message to an Azure Service Bus topic. The collection includes a single request named "AzureSendMessage" which performs the following actions:

Pre-request Script:

Generates a Shared Access Signature (SAS) token for authentication.
Extracts the EventName from the request body and sets it as a label in the BrokerProperties.
Request:

Method: POST
URL: https://<service-bus-name>.servicebus.windows.net/<topic-name>/messages
Headers:
Authorization: Contains the SAS token.
BrokerProperties: Contains the event label.
Body: Sends a JSON payload with various event details, including timestamps, user information, and event-specific data.
Turkish
Bu JSON, bir Azure Service Bus konusuna mesaj gönderen bir Postman koleksiyonudur. Koleksiyon, "AzureSendMessage" adlı tek bir istek içerir ve şu işlemleri gerçekleştirir:

Ön İstek Betiği:

Kimlik doğrulama için Paylaşılan Erişim İmzası (SAS) belirteci oluşturur.
İstek gövdesinden EventName değerini çıkarır ve BrokerProperties içinde etiket olarak ayarlar.
İstek:

Yöntem: POST
URL: https://<service-bus-name>.servicebus.windows.net/<topic-name>/messages
Başlıklar:
Authorization: SAS belirtecini içerir.
BrokerProperties: Olay etiketini içerir.
Gövde: Zaman damgaları, kullanıcı bilgileri ve olaya özgü veriler dahil olmak üzere çeşitli olay ayrıntılarını içeren bir JSON yükü gönderir.
