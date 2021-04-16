---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 820ae9ce7ec4a76891962628086d4eade5ba04cd
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866123"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="2ca30-103">iosLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ca30-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="2ca30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ca30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ca30-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2ca30-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ca30-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ca30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ca30-107">包含用于为组分配 iOS LOB 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="2ca30-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="2ca30-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2ca30-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2ca30-109">属性</span><span class="sxs-lookup"><span data-stu-id="2ca30-109">Properties</span></span>
|<span data-ttu-id="2ca30-110">属性</span><span class="sxs-lookup"><span data-stu-id="2ca30-110">Property</span></span>|<span data-ttu-id="2ca30-111">类型</span><span class="sxs-lookup"><span data-stu-id="2ca30-111">Type</span></span>|<span data-ttu-id="2ca30-112">说明</span><span class="sxs-lookup"><span data-stu-id="2ca30-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ca30-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="2ca30-113">vpnConfigurationId</span></span>|<span data-ttu-id="2ca30-114">String</span><span class="sxs-lookup"><span data-stu-id="2ca30-114">String</span></span>|<span data-ttu-id="2ca30-115">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="2ca30-115">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="2ca30-116">**应用**</span><span class="sxs-lookup"><span data-stu-id="2ca30-116">**Apps**</span></span>|
|<span data-ttu-id="2ca30-117">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="2ca30-117">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="2ca30-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ca30-118">Boolean</span></span>|<span data-ttu-id="2ca30-119">从 Intune 中删除设备时是否卸载应用。</span><span class="sxs-lookup"><span data-stu-id="2ca30-119">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ca30-120">关系</span><span class="sxs-lookup"><span data-stu-id="2ca30-120">Relationships</span></span>
<span data-ttu-id="2ca30-121">无</span><span class="sxs-lookup"><span data-stu-id="2ca30-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ca30-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ca30-122">JSON Representation</span></span>
<span data-ttu-id="2ca30-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ca30-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```




