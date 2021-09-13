---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9920fd26bb9a181d21b09da76c98d0ab37e92b6b727583ae8e1daef4d1f81f81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333806"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemCollectionPage children = graphClient.me().drive().special("{special-folder-name}").children()
    .buildRequest()
    .get();

```