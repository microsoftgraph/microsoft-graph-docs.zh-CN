---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98bdc6ede25b4e6ba6bc4d7ca098a36a84354631
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088436"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deploymentId := "deployment-id"
result, err := graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Get(options)


```