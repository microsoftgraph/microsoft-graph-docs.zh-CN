---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62366d2f4c8d4bd74ad9f227ceea7606364bbbeb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327976"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().MobileAppManagementPolicies().Get()


```