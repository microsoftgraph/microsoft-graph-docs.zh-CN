---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4459dbaf93b1666eb9ca6a8bbe8abfff1faf2d47e46b036f72062b531f56781
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279096"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySettingCollectionPage settings = graphClient.settings()
    .buildRequest()
    .get();

```