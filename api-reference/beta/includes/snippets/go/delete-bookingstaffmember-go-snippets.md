---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5033e15e03d70c14284975735b2d793c8a30f850
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411819"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
bookingStaffMemberId := "bookingStaffMember-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).StaffMembersById(&bookingStaffMemberId).Delete(nil)


```