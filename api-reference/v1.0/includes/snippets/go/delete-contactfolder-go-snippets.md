---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22961ec73deeb077394fca99633d887737346a15
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288542"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

contactFolderId := "contactFolder-id"
graphClient.Me().ContactFoldersById(&contactFolderId).Delete(nil)


```