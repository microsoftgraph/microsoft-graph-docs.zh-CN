---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用程序的安装体验属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aaf3c6dd99b36e33a8af3a8eb4687e1942779937
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538551"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="0c5c3-103">win32LobAppInstallExperience 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c5c3-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="0c5c3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c5c3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c5c3-106">包含 Win32 应用程序的安装体验属性</span><span class="sxs-lookup"><span data-stu-id="0c5c3-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="0c5c3-107">属性</span><span class="sxs-lookup"><span data-stu-id="0c5c3-107">Properties</span></span>
|<span data-ttu-id="0c5c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="0c5c3-108">Property</span></span>|<span data-ttu-id="0c5c3-109">类型</span><span class="sxs-lookup"><span data-stu-id="0c5c3-109">Type</span></span>|<span data-ttu-id="0c5c3-110">说明</span><span class="sxs-lookup"><span data-stu-id="0c5c3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c5c3-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="0c5c3-111">runAsAccount</span></span>|[<span data-ttu-id="0c5c3-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="0c5c3-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="0c5c3-113">指示应用程序在其中运行的执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="0c5c3-114">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-114">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="0c5c3-115">deviceRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="0c5c3-115">deviceRestartBehavior</span></span>|[<span data-ttu-id="0c5c3-116">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="0c5c3-116">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="0c5c3-117">设备重启行为。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-117">Device restart behavior.</span></span> <span data-ttu-id="0c5c3-118">可取值为：`basedOnReturnCode`、`allow`、`suppress`、`force`。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-118">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c5c3-119">关系</span><span class="sxs-lookup"><span data-stu-id="0c5c3-119">Relationships</span></span>
<span data-ttu-id="0c5c3-120">无</span><span class="sxs-lookup"><span data-stu-id="0c5c3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c5c3-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c5c3-121">JSON Representation</span></span>
<span data-ttu-id="0c5c3-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-122">Here is a JSON representation of the resource.</span></span>
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



