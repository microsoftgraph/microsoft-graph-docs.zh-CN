---
title: win32LobAppAssignmentSettings 资源类型
description: 包含用于将 Win32 LOB 移动应用程序分配给组的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2df6ae2cd2543aaea2c095098ea9af2e545f6f92
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004979"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="b60b6-103">win32LobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b60b6-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="b60b6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b60b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b60b6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b60b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b60b6-106">包含用于将 Win32 LOB 移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="b60b6-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="b60b6-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b60b6-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b60b6-108">属性</span><span class="sxs-lookup"><span data-stu-id="b60b6-108">Properties</span></span>
|<span data-ttu-id="b60b6-109">属性</span><span class="sxs-lookup"><span data-stu-id="b60b6-109">Property</span></span>|<span data-ttu-id="b60b6-110">类型</span><span class="sxs-lookup"><span data-stu-id="b60b6-110">Type</span></span>|<span data-ttu-id="b60b6-111">说明</span><span class="sxs-lookup"><span data-stu-id="b60b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b60b6-112">通知</span><span class="sxs-lookup"><span data-stu-id="b60b6-112">notifications</span></span>|[<span data-ttu-id="b60b6-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="b60b6-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="b60b6-114">此应用程序分配的通知状态。</span><span class="sxs-lookup"><span data-stu-id="b60b6-114">The notification status this app assignment.</span></span> <span data-ttu-id="b60b6-115">可取值为：`showAll`、`showReboot`、`hideAll`。</span><span class="sxs-lookup"><span data-stu-id="b60b6-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b60b6-116">关系</span><span class="sxs-lookup"><span data-stu-id="b60b6-116">Relationships</span></span>
<span data-ttu-id="b60b6-117">无</span><span class="sxs-lookup"><span data-stu-id="b60b6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b60b6-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b60b6-118">JSON Representation</span></span>
<span data-ttu-id="b60b6-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b60b6-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String"
}
```





