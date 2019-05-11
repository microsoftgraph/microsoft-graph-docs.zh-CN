---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用程序的安装体验属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc79e79c3922982f58a39b1f835b936e62d5c400
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949582"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="19fa1-103">win32LobAppInstallExperience 资源类型</span><span class="sxs-lookup"><span data-stu-id="19fa1-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="19fa1-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="19fa1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19fa1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19fa1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19fa1-106">包含 Win32 应用程序的安装体验属性</span><span class="sxs-lookup"><span data-stu-id="19fa1-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="19fa1-107">属性</span><span class="sxs-lookup"><span data-stu-id="19fa1-107">Properties</span></span>
|<span data-ttu-id="19fa1-108">属性</span><span class="sxs-lookup"><span data-stu-id="19fa1-108">Property</span></span>|<span data-ttu-id="19fa1-109">类型</span><span class="sxs-lookup"><span data-stu-id="19fa1-109">Type</span></span>|<span data-ttu-id="19fa1-110">说明</span><span class="sxs-lookup"><span data-stu-id="19fa1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19fa1-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="19fa1-111">runAsAccount</span></span>|[<span data-ttu-id="19fa1-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="19fa1-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="19fa1-113">指示应用程序在其中运行的执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="19fa1-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="19fa1-114">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="19fa1-114">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19fa1-115">关系</span><span class="sxs-lookup"><span data-stu-id="19fa1-115">Relationships</span></span>
<span data-ttu-id="19fa1-116">无</span><span class="sxs-lookup"><span data-stu-id="19fa1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19fa1-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19fa1-117">JSON Representation</span></span>
<span data-ttu-id="19fa1-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19fa1-118">Here is a JSON representation of the resource.</span></span>
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




