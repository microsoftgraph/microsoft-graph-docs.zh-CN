---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c7d7a7ffdc19ca072bad8f6ee9309a92fe00805
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137680"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.PrivilegedApproval().MyRequests()().Get(nil)


```