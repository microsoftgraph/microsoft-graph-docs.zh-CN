---
title: deviceManagementUserRightsLocalUserOrGroup 资源类型
description: 表示用于用户权限设置的本地用户或组的信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3bf4ac6aa9de235b1e4117b47c6a5eafc5c011a5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332748"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="02d03-103">deviceManagementUserRightsLocalUserOrGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="02d03-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="02d03-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="02d03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02d03-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02d03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02d03-106">表示用于用户权限设置的本地用户或组的信息。</span><span class="sxs-lookup"><span data-stu-id="02d03-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="02d03-107">属性</span><span class="sxs-lookup"><span data-stu-id="02d03-107">Properties</span></span>
|<span data-ttu-id="02d03-108">属性</span><span class="sxs-lookup"><span data-stu-id="02d03-108">Property</span></span>|<span data-ttu-id="02d03-109">类型</span><span class="sxs-lookup"><span data-stu-id="02d03-109">Type</span></span>|<span data-ttu-id="02d03-110">说明</span><span class="sxs-lookup"><span data-stu-id="02d03-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02d03-111">name</span><span class="sxs-lookup"><span data-stu-id="02d03-111">name</span></span>|<span data-ttu-id="02d03-112">String</span><span class="sxs-lookup"><span data-stu-id="02d03-112">String</span></span>|<span data-ttu-id="02d03-113">此本地用户或组的名称。</span><span class="sxs-lookup"><span data-stu-id="02d03-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="02d03-114">说明</span><span class="sxs-lookup"><span data-stu-id="02d03-114">description</span></span>|<span data-ttu-id="02d03-115">String</span><span class="sxs-lookup"><span data-stu-id="02d03-115">String</span></span>|<span data-ttu-id="02d03-116">管理员对此本地用户或组的说明。</span><span class="sxs-lookup"><span data-stu-id="02d03-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="02d03-117">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="02d03-117">securityIdentifier</span></span>|<span data-ttu-id="02d03-118">String</span><span class="sxs-lookup"><span data-stu-id="02d03-118">String</span></span>|<span data-ttu-id="02d03-119">此本地用户或组的安全标识符 (例如 \* S-1-5-32-544)。</span><span class="sxs-lookup"><span data-stu-id="02d03-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="02d03-120">关系</span><span class="sxs-lookup"><span data-stu-id="02d03-120">Relationships</span></span>
<span data-ttu-id="02d03-121">无</span><span class="sxs-lookup"><span data-stu-id="02d03-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02d03-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02d03-122">JSON Representation</span></span>
<span data-ttu-id="02d03-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02d03-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```



