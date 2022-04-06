---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e79a9e2026ae30deb8d75f7c36f6beb8495707e7
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757966"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveItemId := "driveItem-id"
result, err := graphClient.Drive().BundlesById(&driveItemId).Get(nil)


```