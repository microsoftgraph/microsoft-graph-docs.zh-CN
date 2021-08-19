---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f690e491abeabd1f0b32f19cea4b66945f7c54d01693310db1220df89bc5bdd6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277647"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactCollectionPage contacts = graphClient.me().contacts()
    .buildRequest()
    .get();

```