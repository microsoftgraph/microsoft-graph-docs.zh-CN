---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e57451f9a4d4550413fd6fee263d949ae6909c97
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131722"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingAppointment bookingAppointment = new BookingAppointment();
bookingAppointment.customerEmailAddress = "jordanm@contoso.com";
Location customerLocation = new Location();
PhysicalAddress address = new PhysicalAddress();
address.city = "Buffalo";
address.countryOrRegion = "USA";
address.postalCode = "98052";
address.postOfficeBox = null;
address.state = "NY";
address.street = "123 First Avenue";
address.additionalDataManager().put("type@odata.type", new JsonPrimitive("#microsoft.graph.physicalAddressType"));
address.type = null;
customerLocation.address = address;
customerLocation.coordinates = null;
customerLocation.displayName = "Customer";
customerLocation.locationEmailAddress = null;
customerLocation.additionalDataManager().put("locationType@odata.type", new JsonPrimitive("#microsoft.graph.locationType"));
customerLocation.locationType = null;
customerLocation.locationUri = null;
customerLocation.uniqueId = null;
customerLocation.additionalDataManager().put("uniqueIdType@odata.type", new JsonPrimitive("#microsoft.graph.locationUniqueIdType"));
customerLocation.uniqueIdType = null;
bookingAppointment.customerLocation = customerLocation;
bookingAppointment.customerName = "Jordan Miller";
bookingAppointment.customerNotes = "Please be on time.";
bookingAppointment.customerPhone = "213-555-0199";
bookingAppointment.customerTimeZone = "America/Chicago";
bookingAppointment.smsNotificationsEnabled = true;
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2018-05-01T12:30:00+00:00";
end.timeZone = "UTC";
bookingAppointment.end = end;
bookingAppointment.invoiceAmount = 10.0d;
DateTimeTimeZone invoiceDate = new DateTimeTimeZone();
invoiceDate.dateTime = "2018-05-01T12:30:00+00:00";
invoiceDate.timeZone = "UTC";
bookingAppointment.invoiceDate = invoiceDate;
bookingAppointment.invoiceId = "1001";
bookingAppointment.additionalDataManager().put("invoiceStatus@odata.type", new JsonPrimitive("#microsoft.graph.bookingInvoiceStatus"));
bookingAppointment.invoiceStatus = BookingInvoiceStatus.OPEN;
bookingAppointment.invoiceUrl = "theInvoiceUrl";
bookingAppointment.isLocationOnline = true;
bookingAppointment.optOutOfCustomerEmail = false;
bookingAppointment.postBuffer = DatatypeFactory.newInstance().newDuration("PT10M");
bookingAppointment.preBuffer = DatatypeFactory.newInstance().newDuration("PT5M");
bookingAppointment.price = 10.0d;
bookingAppointment.additionalDataManager().put("priceType@odata.type", new JsonPrimitive("#microsoft.graph.bookingPriceType"));
bookingAppointment.priceType = BookingPriceType.FIXED_PRICE;
bookingAppointment.additionalDataManager().put("reminders@odata.type", new JsonPrimitive("#Collection(microsoft.graph.bookingReminder)"));
LinkedList<BookingReminder> remindersList = new LinkedList<BookingReminder>();
BookingReminder reminders = new BookingReminder();
reminders.message = "This service is tomorrow";
reminders.offset = DatatypeFactory.newInstance().newDuration("P1D");
reminders.additionalDataManager().put("recipients@odata.type", new JsonPrimitive("#microsoft.graph.bookingReminderRecipients"));
reminders.recipients = BookingReminderRecipients.ALL_ATTENDEES;
remindersList.add(reminders);
BookingReminder reminders1 = new BookingReminder();
reminders1.message = "Please be available to enjoy your lunch service.";
reminders1.offset = DatatypeFactory.newInstance().newDuration("PT1H");
reminders1.additionalDataManager().put("recipients@odata.type", new JsonPrimitive("#microsoft.graph.bookingReminderRecipients"));
reminders1.recipients = BookingReminderRecipients.CUSTOMER;
remindersList.add(reminders1);
BookingReminder reminders2 = new BookingReminder();
reminders2.message = "Please check traffic for next cater.";
reminders2.offset = DatatypeFactory.newInstance().newDuration("PT2H");
reminders2.additionalDataManager().put("recipients@odata.type", new JsonPrimitive("#microsoft.graph.bookingReminderRecipients"));
reminders2.recipients = BookingReminderRecipients.STAFF;
remindersList.add(reminders2);
bookingAppointment.reminders = remindersList;
bookingAppointment.serviceId = "57da6774-a087-4d69-b0e6-6fb82c339976";
Location serviceLocation = new Location();
PhysicalAddress address1 = new PhysicalAddress();
address1.city = "Buffalo";
address1.countryOrRegion = "USA";
address1.postalCode = "98052";
address1.postOfficeBox = null;
address1.state = "NY";
address1.street = "123 First Avenue";
address1.additionalDataManager().put("type@odata.type", new JsonPrimitive("#microsoft.graph.physicalAddressType"));
address1.type = null;
serviceLocation.address = address1;
serviceLocation.coordinates = null;
serviceLocation.displayName = "Customer location";
serviceLocation.locationEmailAddress = null;
serviceLocation.additionalDataManager().put("locationType@odata.type", new JsonPrimitive("#microsoft.graph.locationType"));
serviceLocation.locationType = null;
serviceLocation.locationUri = null;
serviceLocation.uniqueId = null;
serviceLocation.additionalDataManager().put("uniqueIdType@odata.type", new JsonPrimitive("#microsoft.graph.locationUniqueIdType"));
serviceLocation.uniqueIdType = null;
bookingAppointment.serviceLocation = serviceLocation;
bookingAppointment.serviceName = "Catered bento";
bookingAppointment.serviceNotes = "Customer requires punctual service.";
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2018-05-01T12:00:00+00:00";
start.timeZone = "UTC";
bookingAppointment.start = start;
bookingAppointment.maximumAttendeesCount = 5;
bookingAppointment.filledAttendeesCount = 1;
LinkedList<BookingCustomerInformationBase> customersList = new LinkedList<BookingCustomerInformationBase>();
BookingCustomerInformation customers = new BookingCustomerInformation();
customers.customerId = "7ed53fa5-9ef2-4f2f-975b-27447440bc09";
customers.name = "Jordan Miller";
customers.emailAddress = "jordanm@contoso.com";
customers.phone = "213-555-0199";
customers.notes = null;
Location location = new Location();
location.displayName = "Customer";
location.locationEmailAddress = null;
location.locationUri = "";
location.locationType = null;
location.uniqueId = null;
location.uniqueIdType = null;
PhysicalAddress address2 = new PhysicalAddress();
address2.type = PhysicalAddressType.HOME;
address2.postOfficeBox = "";
address2.street = "";
address2.city = "";
address2.state = "";
address2.countryOrRegion = "";
address2.postalCode = "";
location.address = address2;
OutlookGeoCoordinates coordinates2 = new OutlookGeoCoordinates();
coordinates2.altitude = 0d;
coordinates2.latitude = 0d;
coordinates2.longitude = 0d;
coordinates2.accuracy = 0d;
coordinates2.altitudeAccuracy = 0d;
location.coordinates = coordinates2;
customers.location = location;
customers.timeZone = "America/Chicago";
LinkedList<BookingQuestionAnswer> customQuestionAnswersList = new LinkedList<BookingQuestionAnswer>();
BookingQuestionAnswer customQuestionAnswers = new BookingQuestionAnswer();
customQuestionAnswers.questionId = "3bc6fde0-4ad3-445d-ab17-0fc15dba0774";
customQuestionAnswers.question = "What is your age";
customQuestionAnswers.answerInputType = AnswerInputType.TEXT;
LinkedList<String> answerOptionsList = new LinkedList<String>();
customQuestionAnswers.answerOptions = answerOptionsList;
customQuestionAnswers.isRequired = true;
customQuestionAnswers.answer = "25";
LinkedList<String> selectedOptionsList = new LinkedList<String>();
customQuestionAnswers.selectedOptions = selectedOptionsList;
customQuestionAnswersList.add(customQuestionAnswers);
customers.customQuestionAnswers = customQuestionAnswersList;
customersList.add(customers);
bookingAppointment.customers = customersList;

graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").appointments()
    .buildRequest()
    .post(bookingAppointment);

```