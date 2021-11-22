---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2848a3eab5185fe9001126ad4d340f38801f68697a75e9c807a8fd787b312d60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221296"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkPositionCollectionPage positions = graphClient.me().profile().positions()
    .buildRequest()
    .get();

```