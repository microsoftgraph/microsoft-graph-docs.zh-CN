---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a7253d8e40ef699bc1066c57c4c423c79a069142
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967894"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="d9be3-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9be3-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="d9be3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d9be3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9be3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9be3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9be3-106">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d9be3-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="d9be3-107">属性</span><span class="sxs-lookup"><span data-stu-id="d9be3-107">Properties</span></span>
|<span data-ttu-id="d9be3-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9be3-108">Property</span></span>|<span data-ttu-id="d9be3-109">类型</span><span class="sxs-lookup"><span data-stu-id="d9be3-109">Type</span></span>|<span data-ttu-id="d9be3-110">说明</span><span class="sxs-lookup"><span data-stu-id="d9be3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9be3-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="d9be3-111">subjectName</span></span>|<span data-ttu-id="d9be3-112">String</span><span class="sxs-lookup"><span data-stu-id="d9be3-112">String</span></span>|<span data-ttu-id="d9be3-113">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="d9be3-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="d9be3-114">说明</span><span class="sxs-lookup"><span data-stu-id="d9be3-114">description</span></span>|<span data-ttu-id="d9be3-115">String</span><span class="sxs-lookup"><span data-stu-id="d9be3-115">String</span></span>|<span data-ttu-id="d9be3-116">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="d9be3-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="d9be3-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d9be3-117">expirationDateTime</span></span>|<span data-ttu-id="d9be3-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9be3-118">DateTimeOffset</span></span>|<span data-ttu-id="d9be3-119">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="d9be3-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="d9be3-120">证书</span><span class="sxs-lookup"><span data-stu-id="d9be3-120">certificate</span></span>|<span data-ttu-id="d9be3-121">Binary</span><span class="sxs-lookup"><span data-stu-id="d9be3-121">Binary</span></span>|<span data-ttu-id="d9be3-122">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="d9be3-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9be3-123">关系</span><span class="sxs-lookup"><span data-stu-id="d9be3-123">Relationships</span></span>
<span data-ttu-id="d9be3-124">无</span><span class="sxs-lookup"><span data-stu-id="d9be3-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9be3-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9be3-125">JSON Representation</span></span>
<span data-ttu-id="d9be3-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9be3-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```





