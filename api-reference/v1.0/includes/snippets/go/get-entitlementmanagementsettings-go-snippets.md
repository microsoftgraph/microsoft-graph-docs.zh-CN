---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3f3d6b5fed3c99703d8e1e73b5d81dd1afb4d5f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327793"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.IdentityGovernance().EntitlementManagement().Settings().Get()


```