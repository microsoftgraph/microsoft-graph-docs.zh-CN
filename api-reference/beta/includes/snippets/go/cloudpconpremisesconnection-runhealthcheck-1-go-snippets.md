---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7eaa2036c6229c022928b74b35a9048c91d0af3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024981"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

cloudPCId := "cloudPC-id"
graphClient.DeviceManagement().VirtualEndpoint().CloudPCsById(&cloudPCId).Reprovision().Post(options)


```