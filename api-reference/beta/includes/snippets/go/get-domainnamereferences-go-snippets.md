---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5bc6348db63c3c978e309fd737491c99dc91043
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022405"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

domainId := "domain-id"
result, err := graphClient.DomainsById(&domainId).DomainNameReferences().Get(options)


```