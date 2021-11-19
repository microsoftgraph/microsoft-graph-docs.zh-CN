---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a168d778851c7af61d008805a2c9c3527e35cbc1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094890"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deploymentId := "deployment-id"
graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Delete(options)


```