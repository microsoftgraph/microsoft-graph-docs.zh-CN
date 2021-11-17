---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbe7a7639e1c1ff20e6e5840a259d2700ab4433596370c8751df70edec1b7fe0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105211"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.me().drive()
    .buildRequest()
    .get();

```