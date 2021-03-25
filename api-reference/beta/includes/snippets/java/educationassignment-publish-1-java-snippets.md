---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f25b864ec5141b63603b16e467ad44a21795a37
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210011"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String string = graphClient.education().classes("11012").assignments("19002")
    .getResourcesFolderUrl()
    .buildRequest()
    .get();

```