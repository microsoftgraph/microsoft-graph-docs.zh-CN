---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb588972eb8304d122f9ccffab7b9a04c2f27079
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288075"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().MobileDeviceManagementPolicies().Get(nil)


```