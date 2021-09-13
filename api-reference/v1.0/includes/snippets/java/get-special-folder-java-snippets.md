---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eff9612025f877cd1f4635cdc3054d8281442875ff22f60c183193da920bc4e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333811"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.me().drive().special("{name}")
    .buildRequest()
    .get();

```