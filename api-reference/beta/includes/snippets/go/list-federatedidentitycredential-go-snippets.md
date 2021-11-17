---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2911755a679b0ace89a95d23eb1cbd519c51e46d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990911"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).FederatedIdentityCredentials().Get(options)


```