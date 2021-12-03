---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee0291b68afda063a4aa5ab4055c53df82f5909b
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287814"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directorySettingId := "directorySetting-id"
result, err := graphClient.SettingsById(&directorySettingId).Get(nil)


```