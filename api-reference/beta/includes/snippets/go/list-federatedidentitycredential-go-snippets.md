---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f7d4273e5a80b15b1f646e889a85ce767d30a5f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096667"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).FederatedIdentityCredentials().Get(options)


```