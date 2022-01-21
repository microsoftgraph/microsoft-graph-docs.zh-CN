---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fdc90eadb4da05a069fee79adc4a749239f2bcb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137714"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.DeviceManagement().VirtualEndpoint().AuditEvents().GetAuditActivityTypes()().Get(nil)


```