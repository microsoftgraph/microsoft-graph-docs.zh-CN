---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用程序的安装体验属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 893f473f7543d93572800776d5511371f7cfbf4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490698"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="81873-103">win32LobAppInstallExperience 资源类型</span><span class="sxs-lookup"><span data-stu-id="81873-103">win32LobAppInstallExperience resource type</span></span>

<span data-ttu-id="81873-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="81873-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81873-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81873-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81873-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81873-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81873-107">包含 Win32 应用程序的安装体验属性</span><span class="sxs-lookup"><span data-stu-id="81873-107">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="81873-108">属性</span><span class="sxs-lookup"><span data-stu-id="81873-108">Properties</span></span>
|<span data-ttu-id="81873-109">属性</span><span class="sxs-lookup"><span data-stu-id="81873-109">Property</span></span>|<span data-ttu-id="81873-110">类型</span><span class="sxs-lookup"><span data-stu-id="81873-110">Type</span></span>|<span data-ttu-id="81873-111">说明</span><span class="sxs-lookup"><span data-stu-id="81873-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81873-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="81873-112">runAsAccount</span></span>|[<span data-ttu-id="81873-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="81873-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="81873-114">指示应用程序在其中运行的执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="81873-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="81873-115">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="81873-115">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="81873-116">deviceRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="81873-116">deviceRestartBehavior</span></span>|[<span data-ttu-id="81873-117">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="81873-117">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="81873-118">设备重启行为。</span><span class="sxs-lookup"><span data-stu-id="81873-118">Device restart behavior.</span></span> <span data-ttu-id="81873-119">可取值为：`basedOnReturnCode`、`allow`、`suppress`、`force`。</span><span class="sxs-lookup"><span data-stu-id="81873-119">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81873-120">关系</span><span class="sxs-lookup"><span data-stu-id="81873-120">Relationships</span></span>
<span data-ttu-id="81873-121">无</span><span class="sxs-lookup"><span data-stu-id="81873-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81873-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81873-122">JSON Representation</span></span>
<span data-ttu-id="81873-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81873-123">Here is a JSON representation of the resource.</span></span>
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



