---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f48465bc8c794a31af7ab7f8034ec5a2cddde37f158de0cdec8381c6e07b7d3b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334128"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directory().deletedItems("{object-id}")
    .buildRequest()
    .get();

```