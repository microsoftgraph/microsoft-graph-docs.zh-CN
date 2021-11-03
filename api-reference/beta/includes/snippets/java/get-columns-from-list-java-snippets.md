---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c2c4e1a06e827d0d8d647042754b021a6127640aa91ada54d528cae15baadfd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162206"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinitionCollectionPage columns = graphClient.sites("{site-id}").lists("{list-id}").columns()
    .buildRequest()
    .get();

```