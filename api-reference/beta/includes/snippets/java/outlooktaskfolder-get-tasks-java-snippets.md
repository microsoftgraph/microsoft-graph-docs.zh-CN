---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 710bb890fbcec4e76bb637684793d966137a2cba65c35a9465f3d36d9a998661
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219735"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskCollectionPage tasks = graphClient.me().outlook().taskFolders("AAMkADIyAAAhrbPWAAA=").tasks()
    .buildRequest()
    .get();

```