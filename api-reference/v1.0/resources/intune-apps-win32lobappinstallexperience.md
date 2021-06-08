---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用的安装体验属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5a1f844683368d898be7a3acdc1dacbcaffa99ff
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760298"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="40096-103">win32LobAppInstallExperience 资源类型</span><span class="sxs-lookup"><span data-stu-id="40096-103">win32LobAppInstallExperience resource type</span></span>

<span data-ttu-id="40096-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40096-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40096-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40096-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40096-106">包含 Win32 应用的安装体验属性</span><span class="sxs-lookup"><span data-stu-id="40096-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="40096-107">属性</span><span class="sxs-lookup"><span data-stu-id="40096-107">Properties</span></span>
|<span data-ttu-id="40096-108">属性</span><span class="sxs-lookup"><span data-stu-id="40096-108">Property</span></span>|<span data-ttu-id="40096-109">类型</span><span class="sxs-lookup"><span data-stu-id="40096-109">Type</span></span>|<span data-ttu-id="40096-110">说明</span><span class="sxs-lookup"><span data-stu-id="40096-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40096-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="40096-111">runAsAccount</span></span>|[<span data-ttu-id="40096-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="40096-112">runAsAccountType</span></span>](../resources/intune-apps-runasaccounttype.md)|<span data-ttu-id="40096-113">指示应用程序运行在的执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="40096-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="40096-114">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="40096-114">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="40096-115">deviceRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="40096-115">deviceRestartBehavior</span></span>|[<span data-ttu-id="40096-116">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="40096-116">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="40096-117">设备重启行为。</span><span class="sxs-lookup"><span data-stu-id="40096-117">Device restart behavior.</span></span> <span data-ttu-id="40096-118">可取值为：`basedOnReturnCode`、`allow`、`suppress`、`force`。</span><span class="sxs-lookup"><span data-stu-id="40096-118">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40096-119">关系</span><span class="sxs-lookup"><span data-stu-id="40096-119">Relationships</span></span>
<span data-ttu-id="40096-120">无</span><span class="sxs-lookup"><span data-stu-id="40096-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40096-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40096-121">JSON Representation</span></span>
<span data-ttu-id="40096-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40096-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String",
  "deviceRestartBehavior": "String"
}
```




