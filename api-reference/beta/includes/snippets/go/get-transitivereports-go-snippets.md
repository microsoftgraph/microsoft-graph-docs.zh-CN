---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 717b5f0190d8f4799f35aed481b8098432029da3
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528083"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

orgContactId := "orgContact-id"
graphClient.ContactsById(&orgContactId).TransitiveReports().$count().Get(nil)


```