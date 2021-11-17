---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d9d7192dbea13e76c5312742b6b1b84814f02fff2898f525d3f2436e834b44e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163598"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrustFrameworkKeySet trustFrameworkKeySet = graphClient.trustFramework().keySets("{id}")
    .buildRequest()
    .get();

```