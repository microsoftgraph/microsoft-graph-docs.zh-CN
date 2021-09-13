---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07ebc186d13cf24924bd1759524480eb9d0526a2863fe008145952b445c4fb51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274287"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveRecentCollectionPage recent = graphClient.me().drive()
    .recent()
    .buildRequest()
    .get();

```