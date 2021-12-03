---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7125e699a50e803a491acf372b96132d8e49213a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288415"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

windowsProtectionStateId := "windowsProtectionState-id"
result, err := graphClient.TenantRelationships().ManagedTenants().WindowsProtectionStatesById(&windowsProtectionStateId).Get(nil)


```