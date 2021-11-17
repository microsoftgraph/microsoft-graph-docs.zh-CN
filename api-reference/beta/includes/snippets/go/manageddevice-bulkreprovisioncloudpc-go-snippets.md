---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe31f5ebfb9f78a16f99d66bea9515330cbac508
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030056"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

graphClient.DeviceManagement().ManagedDevices().BulkReprovisionCloudPc().Post(options)


```