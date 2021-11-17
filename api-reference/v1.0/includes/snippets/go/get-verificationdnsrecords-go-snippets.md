---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bc314e5e0a56a9bc674cd1a8754d878314fc32c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61000403"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

domainId := "domain-id"
result, err := graphClient.DomainsById(&domainId).VerificationDnsRecords().Get(options)


```