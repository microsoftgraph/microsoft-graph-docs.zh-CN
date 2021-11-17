---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40a2cec6b2f9055bd6e38598aaecdb5bce683e5b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994502"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

deviceId := "device-id"
graphClient.DevicesById(&deviceId).Delete(options)


```