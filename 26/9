<?xml version="1.0"?>
<xsd:schema xmlns:xsd="http://www.w3.org/2001/XMLSchema"
            targetNamespace="http://www.student.com"
            xmlns="http://www.student.com"
            elementFormDefault="qualified">

    <xsd:simpleType name="nameType">
        <xsd:restriction base="xsd:string">
            <xsd:pattern value="\p{Lu}(\p{Ll})+\s\p{Lu}(\p{Ll})+"/>
        </xsd:restriction>
    </xsd:simpleType>

    <xsd:simpleType name="genderType">
        <xsd:restriction base="xsd:string">
            <xsd:pattern value="Male|Female" />
        </xsd:restriction>
    </xsd:simpleType>

    <xsd:simpleType name="phoneNoType">
        <xsd:restriction base="xsd:string">
            <xsd:pattern value="\d{3}-\d{7}"/>
        </xsd:restriction>
    </xsd:simpleType>

    <xsd:simpleType name="semmesterType">
        <xsd:restriction base="xsd:integer">
            <xsd:minInclusive value="1" />
            <xsd:maxInclusive value="2" />
        </xsd:restriction>
    </xsd:simpleType>

    <xsd:simpleType name="classSizeType">
        <xsd:restriction base="xsd:integer">
            <xsd:minInclusive value="2" />
            <xsd:maxInclusive value="30" />
        </xsd:restriction>
    </xsd:simpleType>

    <xsd:simpleType name="collegeNameType">
        <xsd:restriction base="xsd:string">
            <xsd:enumeration value="AIT"/>
            <xsd:enumeration value="DIT"/>
            <xsd:enumeration value="NUIG"/>
            <xsd:enumeration value="GMIT"/>
        </xsd:restriction>
    </xsd:simpleType>

    <xsd:simpleType name="favouriteSubjectType">
        <xsd:restriction base="xsd:string">
            <xsd:enumeration value="SOA"/>
            <xsd:enumeration value="Data Science"/>
            <xsd:enumeration value="Agile Build and Delivery"/>
            <xsd:enumeration value="Computer Networks/Telecoms"/>
            <xsd:enumeration value="Software Design"/>
        </xsd:restriction>
    </xsd:simpleType>

    <xsd:simpleType name="studentIDType">
        <xsd:restriction base="xsd:string">
            <xsd:pattern value="A0\d{5}"/>
        </xsd:restriction>
    </xsd:simpleType>
    
    <xsd:element name="student">				
        <xsd:complexType>
            <xsd:sequence>	
                <xsd:element name="personal">				
                    <xsd:complexType>
                        <xsd:sequence>	
                            <xsd:element name="name" type="nameType" />				
                            <xsd:element name="dob" type="xsd:date" />				
                            <xsd:element name="time" type="xsd:time" />	
                            <xsd:element name="gender" type="genderType" />
                            <xsd:element name="weight" type="xsd:double" />
                            <xsd:element name="phoneNo" type="phoneNoType" />			
                        </xsd:sequence>	
                    </xsd:complexType>
                </xsd:element>	
                <xsd:element name="college">
                    <xsd:complexType>
                        <xsd:sequence>	
                            <xsd:element name="course">
                                <xsd:complexType>
                                    <xsd:sequence>	
                                        <xsd:element name="semmester" type="semmesterType" />			
                                        <xsd:element name="classSize" type="classSizeType" />			
                                        <xsd:element name="favouriteSubject" type="favouriteSubjectType" />			
                                    </xsd:sequence>	
                                    <xsd:attribute name="name" type="xsd:string" />
                                </xsd:complexType>
                            </xsd:element>			
                        </xsd:sequence>	
                        <xsd:attribute name="name" type="collegeNameType" />
                        <xsd:attribute name="studentID" type="studentIDType" />
                    </xsd:complexType>
                </xsd:element>			
            </xsd:sequence>
        </xsd:complexType>	
    </xsd:element>
</xsd:schema>


