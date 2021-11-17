---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f1e51b0346873746aeaa9853e38124541f214ba
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018032"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamsAppId := "teamsApp-id"
teamsAppDefinitionId := "teamsAppDefinition-id"
result, err := graphClient.AppCatalogs().TeamsAppsById(&teamsAppId).AppDefinitionsById(&teamsAppDefinitionId).OutlineIcon().Get(options)


```