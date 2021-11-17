---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e757ceafe27bec82762ca4496e579144316c9cec
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033970"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

personAnnualEventId := "personAnnualEvent-id"
graphClient.Me().Profile().AnniversariesById(&personAnnualEventId).Delete(options)


```