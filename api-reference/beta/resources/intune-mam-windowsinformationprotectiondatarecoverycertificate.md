---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae0e8f6f09470d58669acb5123e25a13c6a51dd9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207258"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="f6236-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6236-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="f6236-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6236-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6236-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6236-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6236-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6236-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6236-107">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="f6236-107">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="f6236-108">属性</span><span class="sxs-lookup"><span data-stu-id="f6236-108">Properties</span></span>
|<span data-ttu-id="f6236-109">属性</span><span class="sxs-lookup"><span data-stu-id="f6236-109">Property</span></span>|<span data-ttu-id="f6236-110">类型</span><span class="sxs-lookup"><span data-stu-id="f6236-110">Type</span></span>|<span data-ttu-id="f6236-111">说明</span><span class="sxs-lookup"><span data-stu-id="f6236-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6236-112">SubjectName</span><span class="sxs-lookup"><span data-stu-id="f6236-112">subjectName</span></span>|<span data-ttu-id="f6236-113">String</span><span class="sxs-lookup"><span data-stu-id="f6236-113">String</span></span>|<span data-ttu-id="f6236-114">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="f6236-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="f6236-115">description</span><span class="sxs-lookup"><span data-stu-id="f6236-115">description</span></span>|<span data-ttu-id="f6236-116">String</span><span class="sxs-lookup"><span data-stu-id="f6236-116">String</span></span>|<span data-ttu-id="f6236-117">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="f6236-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="f6236-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f6236-118">expirationDateTime</span></span>|<span data-ttu-id="f6236-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6236-119">DateTimeOffset</span></span>|<span data-ttu-id="f6236-120">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="f6236-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="f6236-121">证书</span><span class="sxs-lookup"><span data-stu-id="f6236-121">certificate</span></span>|<span data-ttu-id="f6236-122">Binary</span><span class="sxs-lookup"><span data-stu-id="f6236-122">Binary</span></span>|<span data-ttu-id="f6236-123">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="f6236-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6236-124">关系</span><span class="sxs-lookup"><span data-stu-id="f6236-124">Relationships</span></span>
<span data-ttu-id="f6236-125">无</span><span class="sxs-lookup"><span data-stu-id="f6236-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6236-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6236-126">JSON Representation</span></span>
<span data-ttu-id="f6236-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6236-127">Here is a JSON representation of the resource.</span></span>
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




