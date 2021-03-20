---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a8b2d730b410964b8fe02fc5ca0485b4cc25234
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951823"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String string = graphClient.education().classes("11012").assignments("19002")
    .getResourcesFolderUrl()
    .buildRequest()
    .get();

```