---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2615e87b646afe689dcf23326f888f804a7a00155a05c9b1a84b7c9961bd91b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902486"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RegionalAndLanguageSettings regionalAndLanguageSettings = graphClient.me().settings().regionalAndLanguageSettings()
    .buildRequest()
    .get();

```