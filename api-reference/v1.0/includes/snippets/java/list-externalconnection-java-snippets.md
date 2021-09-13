---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b5b637020bba27e1c8d60c6989aca859ff3efed27c979cb656c0d96f20b976a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332596"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnectionCollectionPage connections = graphClient.connections()
    .buildRequest()
    .get();

```