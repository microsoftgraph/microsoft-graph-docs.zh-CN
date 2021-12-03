---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a4980e018e132ef0195d51f4cc95db919be4df7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288169"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
userFlowLanguageConfigurationId := "userFlowLanguageConfiguration-id"
result, err := graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).LanguagesById(&userFlowLanguageConfigurationId).OverridesPages().Get(nil)


```