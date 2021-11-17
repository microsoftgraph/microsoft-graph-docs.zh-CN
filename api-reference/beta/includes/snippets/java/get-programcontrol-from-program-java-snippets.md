---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb67a5c3a6cffada6fbfaa64425fc7b6eb363bfef37a24200da494e080e770f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105528"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProgramControlCollectionPage controls = graphClient.programs("673a7379-9c38-4f01-bd9d-4fda7260b807").controls()
    .buildRequest()
    .get();

```