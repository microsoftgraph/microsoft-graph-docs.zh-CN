---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef4ca5e658a31b4b3e04cf52cd67275048b60d4e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017925"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamsAppId := "teamsApp-id"
teamsAppDefinitionId := "teamsAppDefinition-id"
result, err := graphClient.AppCatalogs().TeamsAppsById(&teamsAppId).AppDefinitionsById(&teamsAppDefinitionId).Bot().Get(options)


```