---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed60e9672b567c0278e5bbbfb1c7c26131f07ef8c506f16734fb9198329ba45a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218982"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonWebsiteCollectionPage websites = graphClient.me().profile().websites()
    .buildRequest()
    .get();

```