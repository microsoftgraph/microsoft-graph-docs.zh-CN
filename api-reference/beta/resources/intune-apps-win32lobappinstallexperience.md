---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用程序的安装体验属性
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9eeadf7bc97f53278ef59fe06795bc7120d5bc2c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986297"
---
# <a name="win32lobappinstallexperience-resource-type"></a>win32LobAppInstallExperience 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含 Win32 应用程序的安装体验属性
## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文中运行的应用程序的类型。 可取值为：`system`、`user`。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String"
}
```





