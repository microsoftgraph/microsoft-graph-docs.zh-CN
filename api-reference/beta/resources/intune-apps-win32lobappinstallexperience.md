---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用程序的安装体验属性
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01402384c2628e1f53a854fa35097415181aaa20
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174945"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="9ea77-103">win32LobAppInstallExperience 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ea77-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="9ea77-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ea77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ea77-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ea77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ea77-106">包含 Win32 应用程序的安装体验属性</span><span class="sxs-lookup"><span data-stu-id="9ea77-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="9ea77-107">属性</span><span class="sxs-lookup"><span data-stu-id="9ea77-107">Properties</span></span>
|<span data-ttu-id="9ea77-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ea77-108">Property</span></span>|<span data-ttu-id="9ea77-109">类型</span><span class="sxs-lookup"><span data-stu-id="9ea77-109">Type</span></span>|<span data-ttu-id="9ea77-110">说明</span><span class="sxs-lookup"><span data-stu-id="9ea77-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ea77-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="9ea77-111">runAsAccount</span></span>|[<span data-ttu-id="9ea77-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="9ea77-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="9ea77-113">指示应用程序在其中运行的执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="9ea77-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="9ea77-114">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="9ea77-114">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ea77-115">Relationships</span><span class="sxs-lookup"><span data-stu-id="9ea77-115">Relationships</span></span>
<span data-ttu-id="9ea77-116">无</span><span class="sxs-lookup"><span data-stu-id="9ea77-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ea77-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ea77-117">JSON Representation</span></span>
<span data-ttu-id="9ea77-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ea77-118">Here is a JSON representation of the resource.</span></span>
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




