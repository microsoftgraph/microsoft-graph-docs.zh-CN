---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用程序的安装体验属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 468afea165645c2fc6a728e5a171b1ef37e9e338
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080079"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="5da6b-103">win32LobAppInstallExperience 资源类型</span><span class="sxs-lookup"><span data-stu-id="5da6b-103">win32LobAppInstallExperience resource type</span></span>

<span data-ttu-id="5da6b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5da6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5da6b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5da6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5da6b-106">包含 Win32 应用程序的安装体验属性</span><span class="sxs-lookup"><span data-stu-id="5da6b-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="5da6b-107">属性</span><span class="sxs-lookup"><span data-stu-id="5da6b-107">Properties</span></span>
|<span data-ttu-id="5da6b-108">属性</span><span class="sxs-lookup"><span data-stu-id="5da6b-108">Property</span></span>|<span data-ttu-id="5da6b-109">类型</span><span class="sxs-lookup"><span data-stu-id="5da6b-109">Type</span></span>|<span data-ttu-id="5da6b-110">说明</span><span class="sxs-lookup"><span data-stu-id="5da6b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5da6b-111">deviceRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="5da6b-111">deviceRestartBehavior</span></span>|[<span data-ttu-id="5da6b-112">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="5da6b-112">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="5da6b-113">设备重启行为。</span><span class="sxs-lookup"><span data-stu-id="5da6b-113">Device restart behavior.</span></span> <span data-ttu-id="5da6b-114">可取值为：`basedOnReturnCode`、`allow`、`suppress`、`force`。</span><span class="sxs-lookup"><span data-stu-id="5da6b-114">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5da6b-115">关系</span><span class="sxs-lookup"><span data-stu-id="5da6b-115">Relationships</span></span>
<span data-ttu-id="5da6b-116">无</span><span class="sxs-lookup"><span data-stu-id="5da6b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5da6b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5da6b-117">JSON Representation</span></span>
<span data-ttu-id="5da6b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5da6b-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "deviceRestartBehavior": "String"
}
```





