---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfd68481ba56b789369ef08cc12d195fba6da463f5313e024ed7adfe39ea42de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158434"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.admin().windows().updates().updatableAssets("{updatableAssetId}")
    .buildRequest()
    .delete();

```