---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88b9151ff9c5e7d81e712fb8b2b4782e03d8923a9b416c8e9afc8d088614fbef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163388"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolderCollectionPage taskFolders = graphClient.me().outlook().taskGroups("AAMkADIyAAAhrbe-AAA=").taskFolders()
    .buildRequest()
    .get();

```