---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22d62962e9d42d30b878c941a2092432acce28e20e3b572237beed7ed06a4327
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903138"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingService = new BookingService
{
    DefaultDuration = new Duration("PT1H30M"),
    DefaultLocation = new Location
    {
        Address = new PhysicalAddress
        {
            City = "Buffalo",
            CountryOrRegion = "USA",
            PostalCode = "98052",
            PostOfficeBox = null,
            State = "NY",
            Street = "4567 First Street",
            Type = null,
            AdditionalData = new Dictionary<string, object>()
            {
                {"type@odata.type", "#microsoft.graph.physicalAddressType"}
            }
        },
        Coordinates = null,
        DisplayName = "Contoso Lunch Delivery",
        LocationEmailAddress = null,
        LocationType = null,
        LocationUri = null,
        UniqueId = null,
        UniqueIdType = null,
        AdditionalData = new Dictionary<string, object>()
        {
            {"locationType@odata.type", "#microsoft.graph.locationType"},
            {"uniqueIdType@odata.type", "#microsoft.graph.locationUniqueIdType"}
        }
    },
    DefaultPrice = 10,
    DefaultPriceType = BookingPriceType.FixedPrice,
    DefaultReminders = new List<BookingReminder>()
    {
        new BookingReminder
        {
            Message = "Please be reminded that this service is tomorrow.",
            Offset = new Duration("P1D"),
            Recipients = BookingReminderRecipients.AllAttendees,
            AdditionalData = new Dictionary<string, object>()
            {
                {"recipients@odata.type", "#microsoft.graph.bookingReminderRecipients"}
            }
        }
    },
    Description = "Individual bento box lunch delivery",
    DisplayName = "Bento",
    IsHiddenFromCustomers = false,
    Notes = "Home-cooked special",
    PostBuffer = new Duration("PT10M"),
    PreBuffer = new Duration("PT5M"),
    SchedulingPolicy = new BookingSchedulingPolicy
    {
        AllowStaffSelection = true,
        MaximumAdvance = new Duration("P10D"),
        MinimumLeadTime = new Duration("PT10H"),
        SendConfirmationsToOwner = true,
        TimeSlotInterval = new Duration("PT1H")
    },
    StaffMemberIds = new List<String>()
    {
        "d90d1e8c-5cfe-48cf-a2d5-966267375b6a",
        "2f5f8794-0b29-45b5-b56a-2eb5ff7aa880"
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"defaultPriceType@odata.type", "#microsoft.graph.bookingPriceType"},
        {"defaultReminders@odata.type", "#Collection(microsoft.graph.bookingReminder)"},
        {"staffMemberIds@odata.type", "#Collection(String)"}
    }
};

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Services
    .Request()
    .AddAsync(bookingService);

```