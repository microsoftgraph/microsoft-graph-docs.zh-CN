---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0fd5735e697dafedf15865e23769008c6676b88
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096285"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

graphClient.DeviceManagement().ManagedDevices().BulkReprovisionCloudPc().Post(options)


```