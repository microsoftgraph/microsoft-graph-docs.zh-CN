---
title: educationPowerSchoolDataProvider 资源
description: 用于在将 PowerSchool 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cee763995dd5a75b64d94e5f170d6fea992c20b5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340563"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="c96a5-103">educationPowerSchoolDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="c96a5-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c96a5-104">用于在将[PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/)用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="c96a5-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="c96a5-105">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="c96a5-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c96a5-106">属性</span><span class="sxs-lookup"><span data-stu-id="c96a5-106">Properties</span></span>

| <span data-ttu-id="c96a5-107">属性</span><span class="sxs-lookup"><span data-stu-id="c96a5-107">Property</span></span> | <span data-ttu-id="c96a5-108">类型</span><span class="sxs-lookup"><span data-stu-id="c96a5-108">Type</span></span> | <span data-ttu-id="c96a5-109">说明</span><span class="sxs-lookup"><span data-stu-id="c96a5-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c96a5-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="c96a5-110">**connectionUrl**</span></span> | <span data-ttu-id="c96a5-111">String</span><span class="sxs-lookup"><span data-stu-id="c96a5-111">String</span></span> | <span data-ttu-id="c96a5-112">指向 PowerSchool 实例的连接 URL。</span><span class="sxs-lookup"><span data-stu-id="c96a5-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="c96a5-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="c96a5-113">**clientId**</span></span> | <span data-ttu-id="c96a5-114">String</span><span class="sxs-lookup"><span data-stu-id="c96a5-114">String</span></span> |  <span data-ttu-id="c96a5-115">用于连接到 PowerSchool 的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="c96a5-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="c96a5-116">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="c96a5-116">**clientSecret**</span></span> | <span data-ttu-id="c96a5-117">String</span><span class="sxs-lookup"><span data-stu-id="c96a5-117">String</span></span> |  <span data-ttu-id="c96a5-118">用于对与 PowerSchool 实例的连接进行身份验证的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="c96a5-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="c96a5-119">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="c96a5-119">**schoolsIds**</span></span> | <span data-ttu-id="c96a5-120">String 集合</span><span class="sxs-lookup"><span data-stu-id="c96a5-120">String collection</span></span> |  <span data-ttu-id="c96a5-121">要同步的学校列表。</span><span class="sxs-lookup"><span data-stu-id="c96a5-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="c96a5-122">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="c96a5-122">**schoolYear**</span></span> | <span data-ttu-id="c96a5-123">String</span><span class="sxs-lookup"><span data-stu-id="c96a5-123">String</span></span> |  <span data-ttu-id="c96a5-124">要同步的学校年。</span><span class="sxs-lookup"><span data-stu-id="c96a5-124">The school year to sync.</span></span> |
| <span data-ttu-id="c96a5-125">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="c96a5-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="c96a5-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="c96a5-126">Boolean</span></span> |  <span data-ttu-id="c96a5-127">指示源是否具有单个学生或教师的多个标识符。</span><span class="sxs-lookup"><span data-stu-id="c96a5-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="c96a5-128">**操作**</span><span class="sxs-lookup"><span data-stu-id="c96a5-128">**customizations**</span></span> | [<span data-ttu-id="c96a5-129">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="c96a5-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="c96a5-130">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="c96a5-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c96a5-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c96a5-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
  "connectionUrl": "String",
  "clientId": "String",
  "clientSecret": "String",
  "schoolsIds": ["String"],
  "schoolYear": "String",
  "allowTeachersInMultipleSchools": "Boolean",
  "customizations": {"@odata.type": "microsoft.graph.educationSynchronizationCustomizations"}
}
```
