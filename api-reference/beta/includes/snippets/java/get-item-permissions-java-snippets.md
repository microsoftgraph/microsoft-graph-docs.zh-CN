---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7daefb38db68cf24b14cbcd3840e9d980f193d9d6d31f430134c6dfed0bbc831
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278169"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionCollectionPage permissions = graphClient.me().drive().items("{item-id}").permissions()
    .buildRequest()
    .get();

```