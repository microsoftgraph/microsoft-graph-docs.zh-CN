---
title: groupPolicyObjectFile 资源类型
description: 由管理员上载的组策略对象文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 26881a87b7f22510acf760ae04f967db021e8730
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524474"
---
# <a name="grouppolicyobjectfile-resource-type"></a><span data-ttu-id="5d873-103">groupPolicyObjectFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d873-103">groupPolicyObjectFile resource type</span></span>

<span data-ttu-id="5d873-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5d873-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d873-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5d873-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d873-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5d873-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d873-107">由管理员上载的组策略对象文件。</span><span class="sxs-lookup"><span data-stu-id="5d873-107">The Group Policy Object file uploaded by admin.</span></span>

## <a name="properties"></a><span data-ttu-id="5d873-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d873-108">Properties</span></span>
|<span data-ttu-id="5d873-109">属性</span><span class="sxs-lookup"><span data-stu-id="5d873-109">Property</span></span>|<span data-ttu-id="5d873-110">类型</span><span class="sxs-lookup"><span data-stu-id="5d873-110">Type</span></span>|<span data-ttu-id="5d873-111">说明</span><span class="sxs-lookup"><span data-stu-id="5d873-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d873-112">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="5d873-112">ouDistinguishedName</span></span>|<span data-ttu-id="5d873-113">String</span><span class="sxs-lookup"><span data-stu-id="5d873-113">String</span></span>|<span data-ttu-id="5d873-114">OU 的可分辨名称。</span><span class="sxs-lookup"><span data-stu-id="5d873-114">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="5d873-115">内容</span><span class="sxs-lookup"><span data-stu-id="5d873-115">content</span></span>|<span data-ttu-id="5d873-116">String</span><span class="sxs-lookup"><span data-stu-id="5d873-116">String</span></span>|<span data-ttu-id="5d873-117">组策略对象文件内容。</span><span class="sxs-lookup"><span data-stu-id="5d873-117">The Group Policy Object file content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d873-118">关系</span><span class="sxs-lookup"><span data-stu-id="5d873-118">Relationships</span></span>
<span data-ttu-id="5d873-119">无</span><span class="sxs-lookup"><span data-stu-id="5d873-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d873-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d873-120">JSON Representation</span></span>
<span data-ttu-id="5d873-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d873-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPolicyObjectFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "ouDistinguishedName": "String",
  "content": "String"
}
```



