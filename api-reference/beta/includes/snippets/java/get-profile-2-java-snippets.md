---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07e7f4a235166aed75e2e8593c22261e4f87263c61326cc196235140afa223ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274142"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Profile profile = graphClient.me().profile()
    .buildRequest()
    .expand("skills($select=displayName)")
    .get();

```