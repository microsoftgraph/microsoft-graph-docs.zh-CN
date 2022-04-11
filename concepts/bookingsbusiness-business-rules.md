---
title: 使用 Microsoft Graph 创建或更新Bookings约会时要遵循的业务规则
description: 本文介绍在 Microsoft Graph 中使用创建或更新Bookings约会 API 时要遵循的业务规则。
ms.localizationpriority: medium
author: kwekua
ms.prod: bookings
doc_type: conceptualPageType
ms.openlocfilehash: e1f4a18fcf48d3d18b90a585f48926df1e6aa264
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755711"
---
# <a name="business-rules-for-bookings-appointments"></a>Bookings约会的业务规则

当非管理员用户在Microsoft Bookings中创建约会时，Bookings使用为日历配置的业务规则。 只有管理员有权替代Bookings规则。

通过 Microsoft Graph API 创建或更新约会的最终用户或应用 (使用应用程序权限) 必须遵守业务规则以防止意外错误。

如果使用具有应用程序权限的 [创建](/graph/api/bookingbusiness-post-appointments) 或 [更新](/graph/api/bookingappointment-update) 约会 API，则必须遵循本文中所述的业务规则。

## <a name="business-settings"></a>业务设置

### <a name="business-hours"></a>营业时间

使用 [Update bookingBusiness](/graph/api/bookingbusiness-update?view=graph-rest-beta&tabs=http) API 修改 **businessHours**。 请注意，不能在工作时间之外设置约会。

### <a name="scheduling-policy"></a>计划策略

有关计划策略的详细信息，请参阅 [bookingSchedulingPolicy](/graph/api/resources/bookingschedulingpolicy)。

**时间增量 (时间段间隔)** 指示约会的持续时间。 验证业务规则时，请确保约会的持续时间与服务中指示的持续时间相同。

**最短提前时间** 指示进行或取消约会之前的最短时间。

**最大潜在顾客时间** 指示约会前的最大时间。  

**允许员工选择** 是，如果用户想要通过约会 API 传递员工成员，则应将 [BookingSchedulingPolicy 资源类型的](/graph/api/resources/bookingschedulingpolicy) **allowStaffSelection** 属性设置为 true。

> [!NOTE]
> 此设置在Bookings Web 应用中称为 **“人员控制**”。

## <a name="service-level-settings"></a>服务级别设置

### <a name="scheduling"></a>计划

在服务级别，计划策略继承自业务。 客户可以选择替代策略。

### <a name="main-policy"></a>主策略  

如果在服务级别和业务级别都存在计划策略，则服务级别策略将优先。

### <a name="partially-set-policies"></a>部分设置策略

如果用户未为服务级别策略设置策略，则默认为业务级别策略设置。

### <a name="pre-buffer"></a>预缓冲区

这是在进行以下约会之前约会所需的额外时间。 在员工日历中，约会的持续时间为“预缓冲时间”+“约会槽时间”。

### <a name="post-buffer"></a>缓冲后

这是上一次约会后约会所需的额外时间。 在员工日历中，约会的持续时间为“约会时段”+“后缓冲时间”。
