---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29246e75dfcafb9e47ae49b2273b22c5ec91f011
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411947"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamsAppId := "teamsApp-id"
teamsAppDefinitionId := "teamsAppDefinition-id"
result, err := graphClient.AppCatalogs().TeamsAppsById(&teamsAppId).AppDefinitionsById(&teamsAppDefinitionId).OutlineIcon().HostedContent().$value().Get(nil)


```