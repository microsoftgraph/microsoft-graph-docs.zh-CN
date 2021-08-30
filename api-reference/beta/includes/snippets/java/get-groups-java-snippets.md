---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4860104dfd5cada609ef1798656b0cc0ec13445b2417f29bdcc7f1584fd90414
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104396"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionPage groups = graphClient.groups()
    .buildRequest()
    .get();

```