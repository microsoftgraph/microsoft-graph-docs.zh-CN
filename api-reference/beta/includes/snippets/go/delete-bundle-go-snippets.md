---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e4c21231caf46e463e69d9324f47105c05b8d38
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411978"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveItemId := "driveItem-id"
result, err := graphClient.Drive().ItemsById(&driveItemId).Delete(nil)


```