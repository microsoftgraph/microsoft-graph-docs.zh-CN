---
title: androidPermissionAction 资源类型
description: 请求的权限时，应采取 Android 应用程序权限和 Android 的操作之间的映射。
author: tfitzmac
ms.openlocfilehash: 90117b30dae765151e79d8ad1c2ae1afaa5a42ff
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331134"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="5d939-103">androidPermissionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d939-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="5d939-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5d939-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d939-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5d939-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d939-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5d939-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d939-107">请求的权限时，应采取 Android 应用程序权限和 Android 的操作之间的映射。</span><span class="sxs-lookup"><span data-stu-id="5d939-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>
## <a name="properties"></a><span data-ttu-id="5d939-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d939-108">Properties</span></span>
|<span data-ttu-id="5d939-109">属性</span><span class="sxs-lookup"><span data-stu-id="5d939-109">Property</span></span>|<span data-ttu-id="5d939-110">类型</span><span class="sxs-lookup"><span data-stu-id="5d939-110">Type</span></span>|<span data-ttu-id="5d939-111">说明</span><span class="sxs-lookup"><span data-stu-id="5d939-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d939-112">权限</span><span class="sxs-lookup"><span data-stu-id="5d939-112">permission</span></span>|<span data-ttu-id="5d939-113">字符串</span><span class="sxs-lookup"><span data-stu-id="5d939-113">String</span></span>|<span data-ttu-id="5d939-114">正式 Android 文档中定义的 android 权限字符串。</span><span class="sxs-lookup"><span data-stu-id="5d939-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="5d939-115">示例 android.permission.READ_CONTACTS。</span><span class="sxs-lookup"><span data-stu-id="5d939-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="5d939-116">action</span><span class="sxs-lookup"><span data-stu-id="5d939-116">action</span></span>|[<span data-ttu-id="5d939-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="5d939-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="5d939-118">Android 权限操作的类型。</span><span class="sxs-lookup"><span data-stu-id="5d939-118">Type of Android permission action.</span></span> <span data-ttu-id="5d939-119">可取值为：`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="5d939-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d939-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="5d939-120">Relationships</span></span>
<span data-ttu-id="5d939-121">无</span><span class="sxs-lookup"><span data-stu-id="5d939-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5d939-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d939-122">JSON Representation</span></span>
<span data-ttu-id="5d939-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d939-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```





