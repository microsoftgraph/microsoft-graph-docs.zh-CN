---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 683e52d75bdd85a0cc47da13e741f81d36c91956
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325780"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.RoleManagement().EntitlementManagement().RoleDefinitions().Get()


```