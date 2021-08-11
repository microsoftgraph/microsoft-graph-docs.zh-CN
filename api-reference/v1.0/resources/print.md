---
title: 打印资源类型
description: 当随附通用打印订阅时，打印功能支持管理打印机和发现可用于在通用打印中管理打印机和打印作业的 printServiceEndpoints。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7ed4858a167a87be40ff31e540d402fa93a44cbd30f6ee6e67e63ed52510b9fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129986"
---
# <a name="print-resource-type"></a>打印资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

当随附通用打印订阅时，打印功能支持管理打印机和发现可用于在通用打印中管理打印机和打印作业的[printServiceEndpoints。](printserviceendpoint.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
| [List connectors](../api/print-list-connectors.md) | [printConnector](printconnector.md) 集合 | 获取打印连接器的列表。 |
| [列出打印机](../api/print-list-printers.md) | [printer](printer.md) 集合 | 获取打印机列表。 |
| [列出共享项](../api/print-list-shares.md) | [printerShare](printershare.md) 集合 | 获取打印机共享的列表。 |
| [列出服务](../api/print-list-services.md) | [printService](printservice.md) 集合 | 获取服务列表。 |
| [创建 printerShare](../api/print-post-shares.md) | [printerShare](printershare.md) | 通过发布到 shares 集合创建新的 **打印机** 共享。 |
| [创建打印机](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | 创建 (通用) 新打印机进行注册。 |
| [更新设置](../api/print-update-settings.md) |  [printSettings](printsettings.md) | 更新通用打印服务的租户范围设置。 |
| [List taskDefinitions](../api/print-list-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) 集合 | 获取在通用打印中创建的 printTaskDefinitions 的租户范围列表。 |
| [Create taskDefinition](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | 创建新的 printTaskDefinition。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|settings|[printSettings](../resources/printsettings.md)|通用打印服务的租户范围设置。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|服务|[printService](printservice.md) 集合|可用的通用打印服务终结点的列表。|
|打印机|[printer](printer.md) 集合|租户中注册的打印机列表。|
|shares|[printerShare](printershare.md) 集合|租户中注册的打印机共享列表。|
|连接器|[printConnector](printconnector.md) 集合|可用打印连接器的列表。|
|operations|[printOperation](../resources/printoperation.md) 集合|长时间运行的打印操作的列表。|
|服务|[printService](../resources/printservice.md) 集合|打印基础结构的各个组件的打印服务实例列表。|
|taskDefinitions|[printTaskDefinition](../resources/printtaskdefinition.md) 集合|在通用打印中发生各种事件时可以触发的任务的抽象定义列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.print",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.print",
  "settings": {
    "@odata.type": "microsoft.graph.printSettings"
  }
}
```

