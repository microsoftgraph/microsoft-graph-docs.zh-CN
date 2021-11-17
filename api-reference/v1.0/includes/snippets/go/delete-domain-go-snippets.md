---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2651bcf09b4d681e72e08e791c08655a90b741f5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979128"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

domainId := "domain-id"
graphClient.DomainsById(&domainId).Delete(options)


```