---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34fd3b01f9174d44238d043f14548e7766f8ef5c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092231"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupSettingId := "groupSetting-id"
result, err := graphClient.GroupSettingsById(&groupSettingId).Get(options)


```