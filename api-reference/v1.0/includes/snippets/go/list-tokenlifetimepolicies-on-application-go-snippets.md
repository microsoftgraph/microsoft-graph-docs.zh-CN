---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4fe7091001b25bba34ff3a3de6e92839f8780f4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009133"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).TokenLifetimePolicies().Get(options)


```