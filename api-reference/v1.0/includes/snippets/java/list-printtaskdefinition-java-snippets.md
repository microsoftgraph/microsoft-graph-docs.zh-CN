---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c9f96c48f8d9c059404df9306fc96cab3526c44d70fcc35989a5f6513f63177
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106028"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskDefinitionCollectionPage taskDefinitions = graphClient.print().taskDefinitions()
    .buildRequest()
    .get();

```