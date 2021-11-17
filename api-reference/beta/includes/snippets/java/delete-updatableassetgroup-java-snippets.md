---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e1584f2a6f1116591d28dc139898c8eda65d979f6d760d08735a487317d3734
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163583"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.admin().windows().updates().updatableAssets("{updatableAssetGroupId}")
    .buildRequest()
    .delete();

```