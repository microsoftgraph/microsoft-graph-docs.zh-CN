---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5af85eecf0d6df13c3c791a414673443d0e676a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001426"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).Delete(options)


```